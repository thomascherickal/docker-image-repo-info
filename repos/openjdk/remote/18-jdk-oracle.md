## `openjdk:18-jdk-oracle`

```console
$ docker pull openjdk@sha256:9474bf319fa4488f1d1585bd0dd2f892048c7ffc3c68939d7e9bc3ef6fa9949b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:80b198dad35eaca5d4a87ddb9745ba439925b072bb41079c40c4189f93a30b29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244311499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c9cfd6c29f170f23ad5b721a9648dcbbfee79f15c50ede08255becf382e545f`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 24 Mar 2022 22:26:17 GMT
ADD file:ebb4986af4fcca0d00738e77d2c814e70536c01a0e02eef98c71e9e3a56c0abd in / 
# Thu, 24 Mar 2022 22:26:18 GMT
CMD ["/bin/bash"]
# Fri, 25 Mar 2022 01:16:47 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 25 Mar 2022 01:17:47 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Fri, 25 Mar 2022 01:17:47 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 25 Mar 2022 01:17:47 GMT
ENV LANG=C.UTF-8
# Fri, 25 Mar 2022 01:17:47 GMT
ENV JAVA_VERSION=18
# Fri, 25 Mar 2022 01:17:57 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18/43f95e8614114aeaa8e8a5fcf20a682d/36/GPL/openjdk-18_linux-x64_bin.tar.gz'; 			downloadSha256='0f60aef7b8504983d6e374fe94d09a7bedcf05ec559e812d801a33bd4ebd23d0'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18/43f95e8614114aeaa8e8a5fcf20a682d/36/GPL/openjdk-18_linux-aarch64_bin.tar.gz'; 			downloadSha256='dff2860ba24c3f70f32ad3ac9b03f768dd28044bbda87c9607654fd03795c2ab'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 25 Mar 2022 01:17:57 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1de6f411eccf5041d90362d2d035abf0e59cf91dce4eacbc37ef0aa52f5b5920`  
		Last Modified: Thu, 24 Mar 2022 22:27:23 GMT  
		Size: 42.1 MB (42111629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbc239737191ccc9950c0b7c7a0aa6dac0a92906c45c8c72d511820cf4cd3b6`  
		Last Modified: Fri, 25 Mar 2022 01:24:51 GMT  
		Size: 13.5 MB (13530268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fed1eb83fd97e7c92eb1f29b7a79f2d9e3bdc98379163f96d739016bb068b7`  
		Last Modified: Fri, 25 Mar 2022 01:26:45 GMT  
		Size: 188.7 MB (188669602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:1eba49f0f791188b0a3a49aa6a5ca26d2b533555c5bc2194ebd6af5dc8db1429
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.9 MB (243905275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f4af77da18184f206c06c9d35070ae25cb13e2de2b82713c96058b0a382a319`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 24 Mar 2022 22:21:09 GMT
ADD file:1eaca9dccdbe88c4fac0b484a625100443af30879cf6cba7b5615db77745b0c7 in / 
# Thu, 24 Mar 2022 22:21:10 GMT
CMD ["/bin/bash"]
# Thu, 24 Mar 2022 22:45:15 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 24 Mar 2022 22:47:13 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 24 Mar 2022 22:47:14 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 22:47:15 GMT
ENV LANG=C.UTF-8
# Thu, 24 Mar 2022 22:47:16 GMT
ENV JAVA_VERSION=18
# Thu, 24 Mar 2022 22:47:27 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk18/43f95e8614114aeaa8e8a5fcf20a682d/36/GPL/openjdk-18_linux-x64_bin.tar.gz'; 			downloadSha256='0f60aef7b8504983d6e374fe94d09a7bedcf05ec559e812d801a33bd4ebd23d0'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk18/43f95e8614114aeaa8e8a5fcf20a682d/36/GPL/openjdk-18_linux-aarch64_bin.tar.gz'; 			downloadSha256='dff2860ba24c3f70f32ad3ac9b03f768dd28044bbda87c9607654fd03795c2ab'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 24 Mar 2022 22:47:27 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c11319b13f376dfb3fa1ee22d0047cfb7157eba4ba2786653cb29ac6defcb93c`  
		Last Modified: Thu, 24 Mar 2022 22:22:26 GMT  
		Size: 42.0 MB (42018948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d7710250d8de942c9ab085f8642e5e854d0b85b2578079aa2a8f4aaac0bf73`  
		Last Modified: Thu, 24 Mar 2022 23:01:12 GMT  
		Size: 14.3 MB (14293656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d8e2159139ae9f7c0341d3c9469101195308de28699704bc6babbfc200d991`  
		Last Modified: Thu, 24 Mar 2022 23:03:31 GMT  
		Size: 187.6 MB (187592671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
