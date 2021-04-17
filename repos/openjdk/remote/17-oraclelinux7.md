## `openjdk:17-oraclelinux7`

```console
$ docker pull openjdk@sha256:892a8380d17605d5f2022b5a47550eda2db813708f0f6f6936fe7c6ddd58d9d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:17-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:9dab4dd3005acceebbf0c1f3f1bc975f72396898d2da59ebd05cc26b7a86319b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.7 MB (249698033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60d0cce536a076b48d5609862fc1817fd21ba89e20f9fcc41c756bc849d5302d`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 17 Mar 2021 00:21:32 GMT
ADD file:837f2bca2cab135736ad43644356710dcac6516fdfc2023d239d157d1fa4ba7c in / 
# Wed, 17 Mar 2021 00:21:32 GMT
CMD ["/bin/bash"]
# Wed, 17 Mar 2021 00:38:33 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 17 Mar 2021 00:38:33 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Wed, 17 Mar 2021 00:38:34 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Mar 2021 00:38:34 GMT
ENV LANG=en_US.UTF-8
# Fri, 16 Apr 2021 22:21:29 GMT
ENV JAVA_VERSION=17-ea+18
# Fri, 16 Apr 2021 22:21:39 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/18/GPL/openjdk-17-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='272350ce50f4f6f5ff111060a05bafa14f1adfe9ea9f0df06ea1cb242760ed29'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/18/GPL/openjdk-17-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='0b65ebc5bcb5e14028c6459bc32158ac530bb41418ca2be95de4da4e64d90df7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 16 Apr 2021 22:21:39 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:401a42e1eb4fe87d89990847d6ef97767b5ac57457c8001203ee2ea137736907`  
		Last Modified: Wed, 17 Mar 2021 00:22:34 GMT  
		Size: 48.3 MB (48263709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f752366003eed4ac964ebb4be3453e3f19d854828f4f50ff708900bb4c42924`  
		Last Modified: Wed, 17 Mar 2021 00:45:21 GMT  
		Size: 15.4 MB (15429957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a2ee869f927608f7a4461ce5c017ae20b32f4befe1160a269810f5de4f8b5e`  
		Last Modified: Fri, 16 Apr 2021 22:27:54 GMT  
		Size: 186.0 MB (186004367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:12e5fe6dc7fd8bc4726dab848e61b7eaceb8f7c9d19fa34a5b1b1ef1793ec656
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.4 MB (247412249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40e07b65e8adeb38969397dc521017daabc9a10a0c2de65fe6c0ea6907e8fdcf`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 17 Mar 2021 03:42:09 GMT
ADD file:035a776cfbed0261290447a1f521123f230f599d8a9ede7feb4616146e47fe10 in / 
# Wed, 17 Mar 2021 03:42:13 GMT
CMD ["/bin/bash"]
# Wed, 17 Mar 2021 04:00:37 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 17 Mar 2021 04:00:38 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Wed, 17 Mar 2021 04:00:39 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Mar 2021 04:00:39 GMT
ENV LANG=en_US.UTF-8
# Fri, 16 Apr 2021 22:41:33 GMT
ENV JAVA_VERSION=17-ea+18
# Fri, 16 Apr 2021 22:41:59 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/18/GPL/openjdk-17-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='272350ce50f4f6f5ff111060a05bafa14f1adfe9ea9f0df06ea1cb242760ed29'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/18/GPL/openjdk-17-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='0b65ebc5bcb5e14028c6459bc32158ac530bb41418ca2be95de4da4e64d90df7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 16 Apr 2021 22:42:01 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d8ef6a6bcc7f4a961a86d5d1f004e51937aa0e6caf0086b892501d0f909ac044`  
		Last Modified: Wed, 17 Mar 2021 03:43:17 GMT  
		Size: 48.9 MB (48853748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4aee6eb11d4d9526fe0e54fda7fb88ac928a854d7984a42bda3cb37c97b5bf0`  
		Last Modified: Wed, 17 Mar 2021 04:07:44 GMT  
		Size: 16.5 MB (16465148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87ee9a9d1d3720e117d3a6d4d17ca4989a6898c2c620b77a353d5a84ae472b1`  
		Last Modified: Fri, 16 Apr 2021 22:47:55 GMT  
		Size: 182.1 MB (182093353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
