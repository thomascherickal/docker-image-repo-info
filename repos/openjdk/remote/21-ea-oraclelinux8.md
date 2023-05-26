## `openjdk:21-ea-oraclelinux8`

```console
$ docker pull openjdk@sha256:995eaa2adb9fc8e7ea33b638404b3dededbb0e804cd49a748079e9dde8d6dd89
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:21-ea-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:f2c33bb04d4126ec8d1eab7f86226b68e9f25058ee510eb25cf72bb5cf97a07e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **263.0 MB (263022860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a737415ec531faa9f3590c2ffe39a3299fe87acd82cc4c2ea132d2b43afb8e2`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 24 May 2023 21:20:28 GMT
ADD file:e15c235506d8dd134e69d458a7c0afefef1522e9d0cfb28e3538760ddf032785 in / 
# Wed, 24 May 2023 21:20:29 GMT
CMD ["/bin/bash"]
# Wed, 24 May 2023 21:44:56 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 24 May 2023 21:44:56 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Wed, 24 May 2023 21:44:56 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 May 2023 21:44:56 GMT
ENV LANG=C.UTF-8
# Fri, 26 May 2023 23:05:09 GMT
ENV JAVA_VERSION=21-ea+24
# Fri, 26 May 2023 23:05:20 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/24/GPL/openjdk-21-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='437e740a3ee795a3cf08d6cf5006d03668023151200d5e09ada16d94ef30db22'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/24/GPL/openjdk-21-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='ecabd8a50340461d04d06b8f587bf06c614aed9cb441ee3ff9577e1b10e53035'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 26 May 2023 23:05:20 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:90e2fb2facff1c5093f0ebfa9d08fde487930822d9ac278bb2df0195610f1d13`  
		Last Modified: Wed, 24 May 2023 21:21:24 GMT  
		Size: 44.9 MB (44873648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0845850e9baa985b97efc76bed4795ff90eb1249ecf4531667da84d4be1fcdf`  
		Last Modified: Wed, 24 May 2023 21:45:40 GMT  
		Size: 15.0 MB (15010668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee812e754920b3231666f1d458d8aef25c9e75562b5b05c314dd1d9778d52ca`  
		Last Modified: Fri, 26 May 2023 23:07:29 GMT  
		Size: 203.1 MB (203138544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:21-ea-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:27f52854c43307c0f923e67f26a1d9f661ac20831b6c724e4de0a6a60eafe279
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.1 MB (261121088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec2089cc4b709fb37808e9d16785253780275e1058d570026a03b68e0529e945`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 24 May 2023 21:44:09 GMT
ADD file:8c6f57a98019c407c59b2adbf7da54536eff3a7ca62c46883bbc60975b39ad04 in / 
# Wed, 24 May 2023 21:44:09 GMT
CMD ["/bin/bash"]
# Wed, 24 May 2023 22:03:14 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 24 May 2023 22:03:14 GMT
ENV JAVA_HOME=/usr/java/openjdk-21
# Wed, 24 May 2023 22:03:14 GMT
ENV PATH=/usr/java/openjdk-21/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 May 2023 22:03:14 GMT
ENV LANG=C.UTF-8
# Thu, 25 May 2023 23:39:43 GMT
ENV JAVA_VERSION=21-ea+24
# Thu, 25 May 2023 23:39:56 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/24/GPL/openjdk-21-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='437e740a3ee795a3cf08d6cf5006d03668023151200d5e09ada16d94ef30db22'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk21/24/GPL/openjdk-21-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='ecabd8a50340461d04d06b8f587bf06c614aed9cb441ee3ff9577e1b10e53035'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 25 May 2023 23:39:58 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:0bb308beee4aa3eb768d546b1ee61303d6f190f63bed75dc7f88ecc26018a944`  
		Last Modified: Wed, 24 May 2023 21:44:58 GMT  
		Size: 43.8 MB (43791991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da95086478e81c9f4c37c04e50d244968af554844dd950bcb04b5f0171653f64`  
		Last Modified: Wed, 24 May 2023 22:03:55 GMT  
		Size: 15.9 MB (15852529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c427e1a7c7546fe45ab6f18696b7bf1e8173249c96d70f910136d2f0663221`  
		Last Modified: Thu, 25 May 2023 23:42:01 GMT  
		Size: 201.5 MB (201476568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
