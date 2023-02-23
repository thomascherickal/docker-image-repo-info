## `openjdk:21-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:8e4a3672a97e5d950c95a8243ae56c965c1daf199417d96d082efc766e297537
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:07f02c9be711e04f8ab59a4a40ab41d47abb5c2cdbd7b964540be886953c428b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.1 MB (256125648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7191613b0bb1eb14f9ae2f9356d1eece7daf36db5a3f526ea27ee17f4ff91223`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 23 Feb 2023 19:37:08 GMT
ADD file:7c92981e2fed9bedfca663209480ce9006dce0edc6c44c25640255683952b929 in / 
# Thu, 23 Feb 2023 19:37:08 GMT
CMD ["/bin/bash"]
# Thu, 23 Feb 2023 19:56:18 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 23 Feb 2023 19:56:18 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Thu, 23 Feb 2023 19:56:18 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Feb 2023 19:56:18 GMT
ENV LANG=C.UTF-8
# Thu, 23 Feb 2023 19:56:19 GMT
ENV JAVA_VERSION=21-ea+10
# Thu, 23 Feb 2023 19:56:29 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/10/GPL/openjdk-21-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='e60198534add038869d333ae9564ff8be298d712c5518b865952d66d07638b7b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/10/GPL/openjdk-21-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='eb5e840f2f81330fa3080312da34ce1daabb27138bbebdbb5ea409d79a970e6c'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 23 Feb 2023 19:56:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1319f85bbd2aad3767d41a6c767c94c23f7432642c7bda3df878c147ba384902`  
		Last Modified: Thu, 23 Feb 2023 19:38:02 GMT  
		Size: 44.6 MB (44552452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565fe2a72fd544bf059ba3dab17c20dd57232b65e41885f9004b841d0106f73b`  
		Last Modified: Thu, 23 Feb 2023 19:58:20 GMT  
		Size: 12.2 MB (12246468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cc176753cc1e165ecfba28a9a7c494cc15e2d19148b3529c58152e4125b66e`  
		Last Modified: Thu, 23 Feb 2023 19:58:32 GMT  
		Size: 199.3 MB (199326728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:9994bb788f77e985701b9845c29b5fc4ba82f8cb00e619fe23ab717dea1e664b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.3 MB (254347152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93f72d04d0e491689a963c3401dbe0d00faea2d33ad19be53160ca99baf16f6f`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 23 Feb 2023 19:52:36 GMT
ADD file:650f46a4a6a15a9b2d6f048bb51976942936d0c5daba7b0337bceacbc4efcf85 in / 
# Thu, 23 Feb 2023 19:52:37 GMT
CMD ["/bin/bash"]
# Thu, 23 Feb 2023 20:13:51 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 23 Feb 2023 20:13:51 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Thu, 23 Feb 2023 20:13:51 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Feb 2023 20:13:51 GMT
ENV LANG=C.UTF-8
# Thu, 23 Feb 2023 20:13:51 GMT
ENV JAVA_VERSION=21-ea+10
# Thu, 23 Feb 2023 20:14:05 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/10/GPL/openjdk-21-ea+10_linux-x64_bin.tar.gz'; 			downloadSha256='e60198534add038869d333ae9564ff8be298d712c5518b865952d66d07638b7b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/10/GPL/openjdk-21-ea+10_linux-aarch64_bin.tar.gz'; 			downloadSha256='eb5e840f2f81330fa3080312da34ce1daabb27138bbebdbb5ea409d79a970e6c'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 23 Feb 2023 20:14:07 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7166504978b203e953381fdfe4d9e7656565d62a75183fcc5bf460e6135e033d`  
		Last Modified: Thu, 23 Feb 2023 19:53:23 GMT  
		Size: 43.5 MB (43459902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766ec681792700cac3beb59912bb93402833e5171c8ae979918ee6806da3d433`  
		Last Modified: Thu, 23 Feb 2023 20:16:05 GMT  
		Size: 13.1 MB (13073314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d49c44a5cd05f075b0bf6db6725e39ff3305ebc272377549029b9483847bbba`  
		Last Modified: Thu, 23 Feb 2023 20:16:16 GMT  
		Size: 197.8 MB (197813936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
