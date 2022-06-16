## `openjdk:20-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:fc4bab716d109cd3ee16d4bd3b495a6887a676fc7803db86cf682a256957dfc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:422720c8bbb83cf3f1be6aaec653c7e80575dea6e694ddfb49c08543d58ed50b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.8 MB (249829090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a41809a34a720e13da58f2aba0a9968a0793a25e029dd8775704514ec692f34e`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 14 Jun 2022 18:23:26 GMT
ADD file:837f6c6e7e20067b92edb72e78a8399e6cbbd72dab23db7b5b5a301c58d2a0de in / 
# Tue, 14 Jun 2022 18:23:26 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 18:42:55 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 16 Jun 2022 01:21:37 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Thu, 16 Jun 2022 01:21:37 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Jun 2022 01:21:37 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jun 2022 01:21:37 GMT
ENV JAVA_VERSION=20-ea+1
# Thu, 16 Jun 2022 01:21:47 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/1/GPL/openjdk-20-ea+1_linux-x64_bin.tar.gz'; 			downloadSha256='0abed92a0e13e5d0f0d02463a90b21a040db83ea57617f5c61c5547862152766'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/1/GPL/openjdk-20-ea+1_linux-aarch64_bin.tar.gz'; 			downloadSha256='898a2f8ca4e530d154e94ca685ef4f03341cd78f3514661a03c8f87bfbdd2371'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 16 Jun 2022 01:21:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5f160c0f6cac587a73883b48a8857f5cce0930112792cef25c62510e256e93dc`  
		Last Modified: Tue, 14 Jun 2022 18:24:18 GMT  
		Size: 39.2 MB (39219730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb499df0377a2bd9163e9a611ce46b5379196826787392defef98dbf215a8aa4`  
		Last Modified: Tue, 14 Jun 2022 18:49:29 GMT  
		Size: 13.5 MB (13502563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50cb76b6da42d4549ad4b08f2159e0fb8b255f3a7e25e5d0ead1fbfdfb03dd98`  
		Last Modified: Thu, 16 Jun 2022 01:30:46 GMT  
		Size: 197.1 MB (197106797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:69801103039ce70d3516d084797b38804f65be0ae337c53edd79ec64ba7de4c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.2 MB (248223429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c6648dc8ba9c1354f1bb6cb3b61a018b8c5f706a560eaf25847b59f0d4726eb`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 14 Jun 2022 18:41:36 GMT
ADD file:4a6ee90ad73353bfb87b2f121e06bddaed6104536e485baa83fadbe7facc774c in / 
# Tue, 14 Jun 2022 18:41:37 GMT
CMD ["/bin/bash"]
# Tue, 14 Jun 2022 18:58:47 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 16 Jun 2022 00:49:01 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Thu, 16 Jun 2022 00:49:02 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Jun 2022 00:49:03 GMT
ENV LANG=C.UTF-8
# Thu, 16 Jun 2022 00:49:04 GMT
ENV JAVA_VERSION=20-ea+1
# Thu, 16 Jun 2022 00:49:16 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/1/GPL/openjdk-20-ea+1_linux-x64_bin.tar.gz'; 			downloadSha256='0abed92a0e13e5d0f0d02463a90b21a040db83ea57617f5c61c5547862152766'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/1/GPL/openjdk-20-ea+1_linux-aarch64_bin.tar.gz'; 			downloadSha256='898a2f8ca4e530d154e94ca685ef4f03341cd78f3514661a03c8f87bfbdd2371'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 16 Jun 2022 00:49:16 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:2bbc1bf883bd601c0da5735b538963308bcc17f90d36525ecc93456ffad79064`  
		Last Modified: Tue, 14 Jun 2022 18:42:39 GMT  
		Size: 38.0 MB (38012371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bde7855ef536fce06527372a019087e1972db9d092b2ec88091b6017cfc5a16`  
		Last Modified: Tue, 14 Jun 2022 19:10:59 GMT  
		Size: 14.3 MB (14260872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24d64b9c0ee7e06064002cd5e17a41f6d4d666c7deb516a120b927c62a6b89c`  
		Last Modified: Thu, 16 Jun 2022 01:04:05 GMT  
		Size: 196.0 MB (195950186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
