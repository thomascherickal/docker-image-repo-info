## `openjdk:18-ea-27-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:67d7cf933058a34efa99c3d282a339bf8a78db97a2856c97ec423ef9a5f38933
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-ea-27-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:b83963517a2ef63e820276a2b0650939bd0f9620f8053c615fcd4bac81aee7db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.3 MB (252297660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad15ce625d781e4bdf94190314b84c51639e71df216b8944c5a98e3ad9e68398`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 02 Dec 2021 03:36:07 GMT
ADD file:f1e23cb77895c4f36fa773b22bdbd74dfd2a144a4da854f13fd100d73f5517d8 in / 
# Thu, 02 Dec 2021 03:36:07 GMT
CMD ["/bin/bash"]
# Thu, 02 Dec 2021 11:28:23 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 02 Dec 2021 11:28:23 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 02 Dec 2021 11:28:24 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 11:28:24 GMT
ENV LANG=en_US.UTF-8
# Fri, 10 Dec 2021 21:20:21 GMT
ENV JAVA_VERSION=18-ea+27
# Fri, 10 Dec 2021 21:20:31 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/27/GPL/openjdk-18-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='625301c146fd49d5f45dae30876079fe01ee959d84573a056426362fd6699f1f'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/27/GPL/openjdk-18-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad926dc5db48de8dce170eb97ed1539d03829b3f23cf4a2a654e0f8f296be8e7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 10 Dec 2021 21:20:32 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:f09c1d3b7e7b9dae0fc06393c0a6ae2becfdaf108965c4634fb5aa08ef682b39`  
		Last Modified: Thu, 02 Dec 2021 03:37:01 GMT  
		Size: 48.3 MB (48330617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a0bdeb652c6947210f8fca8bc5216da702dcb944e14fb6272fde14a87c1834`  
		Last Modified: Thu, 02 Dec 2021 11:46:03 GMT  
		Size: 15.4 MB (15388709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76275c4275108cc1b2047dc3d4eedcb2294a3328050153f4804de88a91ed0a80`  
		Last Modified: Fri, 10 Dec 2021 21:27:36 GMT  
		Size: 188.6 MB (188578334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-27-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:09dad3b2c1725f9d794c28aa43327f80548bc88b8b90a712b80a4bcb990003c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.9 MB (252870483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99856d0b36010c942f8aa57265f3c11de5a854187df88e1971d7593e93b0234d`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 02 Dec 2021 08:51:25 GMT
ADD file:9e54130641553fdfd5c6fccb94502b8821e5f6a3a312a5b58537b439bf8b2670 in / 
# Thu, 02 Dec 2021 08:51:26 GMT
CMD ["/bin/bash"]
# Thu, 02 Dec 2021 11:01:07 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 02 Dec 2021 11:01:08 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Thu, 02 Dec 2021 11:01:09 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Dec 2021 11:01:10 GMT
ENV LANG=en_US.UTF-8
# Fri, 10 Dec 2021 21:52:15 GMT
ENV JAVA_VERSION=18-ea+27
# Fri, 10 Dec 2021 21:52:33 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/27/GPL/openjdk-18-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='625301c146fd49d5f45dae30876079fe01ee959d84573a056426362fd6699f1f'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/27/GPL/openjdk-18-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad926dc5db48de8dce170eb97ed1539d03829b3f23cf4a2a654e0f8f296be8e7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 10 Dec 2021 21:52:33 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:badc99e3da86862c7fae71e717cef8fd1a5a34023f0932c8c979275fb8de6a32`  
		Last Modified: Thu, 02 Dec 2021 08:52:20 GMT  
		Size: 48.9 MB (48905570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56494d755d6c4fa6e0ed158c6946591b3ec2ad7e02e9c86d1434bcf5b27c263`  
		Last Modified: Thu, 02 Dec 2021 11:21:55 GMT  
		Size: 16.5 MB (16464679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e36ff6ac18f40598b6f0b41ca53d1b8b6aa5ed80f7346547dab5e5e2b4eee41`  
		Last Modified: Fri, 10 Dec 2021 22:04:47 GMT  
		Size: 187.5 MB (187500234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
