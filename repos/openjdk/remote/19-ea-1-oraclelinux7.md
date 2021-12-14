## `openjdk:19-ea-1-oraclelinux7`

```console
$ docker pull openjdk@sha256:abe0f5121e66ef6dc04ecc0b27838ddb7f2f898b0ebc877cec09f9c6778ce47f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-1-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:6c3760439348d3a1fd5784bd7253b7f0db043c651d1154e7e57afb198c1bf9d3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.2 MB (253195555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33bc92970448849ce4d3ae866e36f4f210b0c7521de7958a009965c0b0377ca2`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 02 Dec 2021 03:36:07 GMT
ADD file:f1e23cb77895c4f36fa773b22bdbd74dfd2a144a4da854f13fd100d73f5517d8 in / 
# Thu, 02 Dec 2021 03:36:07 GMT
CMD ["/bin/bash"]
# Thu, 02 Dec 2021 11:28:23 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 14 Dec 2021 01:41:26 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Tue, 14 Dec 2021 01:41:26 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Dec 2021 01:41:27 GMT
ENV LANG=en_US.UTF-8
# Tue, 14 Dec 2021 01:41:27 GMT
ENV JAVA_VERSION=19-ea+1
# Tue, 14 Dec 2021 01:41:38 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/1/GPL/openjdk-19-ea+1_linux-x64_bin.tar.gz'; 			downloadSha256='652a141e1854a51df7991b003d6e9478021cb4a4ee67b320cb284e40dff46847'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/1/GPL/openjdk-19-ea+1_linux-aarch64_bin.tar.gz'; 			downloadSha256='fe09452d49aad26e03df3d5b5ebfc22f8b2d8a1e16dcc03a2f00b31f586a770a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 14 Dec 2021 01:41:39 GMT
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
	-	`sha256:f1490d32c95a33e35dfc86dbb494d0686c5bf28e07348d52c9d4d0586080116b`  
		Last Modified: Tue, 14 Dec 2021 01:50:17 GMT  
		Size: 189.5 MB (189476229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-1-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:b43f4fdcf58de07dbc6638230c63b6b2d88b15dd1972d18cd6cafc6614509964
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.8 MB (253786181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:577bd8e300d3a28a7ff20074a66d7d4f8661eef6befa0cb3002141dba3864611`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 02 Dec 2021 08:51:25 GMT
ADD file:9e54130641553fdfd5c6fccb94502b8821e5f6a3a312a5b58537b439bf8b2670 in / 
# Thu, 02 Dec 2021 08:51:26 GMT
CMD ["/bin/bash"]
# Thu, 02 Dec 2021 11:01:07 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 14 Dec 2021 01:59:08 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Tue, 14 Dec 2021 01:59:09 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Dec 2021 01:59:10 GMT
ENV LANG=en_US.UTF-8
# Tue, 14 Dec 2021 01:59:11 GMT
ENV JAVA_VERSION=19-ea+1
# Tue, 14 Dec 2021 01:59:27 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/1/GPL/openjdk-19-ea+1_linux-x64_bin.tar.gz'; 			downloadSha256='652a141e1854a51df7991b003d6e9478021cb4a4ee67b320cb284e40dff46847'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/1/GPL/openjdk-19-ea+1_linux-aarch64_bin.tar.gz'; 			downloadSha256='fe09452d49aad26e03df3d5b5ebfc22f8b2d8a1e16dcc03a2f00b31f586a770a'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 14 Dec 2021 01:59:28 GMT
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
	-	`sha256:d3a67e34ff6fce90008f41994e2d76503aeb67e50af4521a427c775ebb9fe032`  
		Last Modified: Tue, 14 Dec 2021 02:14:05 GMT  
		Size: 188.4 MB (188415932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
