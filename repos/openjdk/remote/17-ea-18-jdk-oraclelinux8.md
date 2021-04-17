## `openjdk:17-ea-18-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:f5a659dc4b61b4782ffc9b7d5a818af9d0d4cd6ba942b6165ace3a6bffdd0ba1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:17-ea-18-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:dd7c4ef0efae41fbcbb8ca197884df5d935895aca7f3c83d1b7240947664995a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241332950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76b2f7b3691641b2b382bcacca26bc29446c927222b9dbe8c91408d667dce9fd`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 30 Mar 2021 21:01:16 GMT
ADD file:6a8b1c26fdbf2beb390286575735d9efcd8cd6c3d135c9d7d25b3fe4c641a7ee in / 
# Tue, 30 Mar 2021 21:01:16 GMT
CMD ["/bin/bash"]
# Tue, 30 Mar 2021 21:36:54 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 30 Mar 2021 21:36:55 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Tue, 30 Mar 2021 21:36:55 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Mar 2021 21:36:55 GMT
ENV LANG=C.UTF-8
# Fri, 16 Apr 2021 22:21:13 GMT
ENV JAVA_VERSION=17-ea+18
# Fri, 16 Apr 2021 22:21:23 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/18/GPL/openjdk-17-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='272350ce50f4f6f5ff111060a05bafa14f1adfe9ea9f0df06ea1cb242760ed29'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/18/GPL/openjdk-17-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='0b65ebc5bcb5e14028c6459bc32158ac530bb41418ca2be95de4da4e64d90df7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 16 Apr 2021 22:21:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:50c2d151af498a24eabbdd1f14042e94106189e17f7858fa9c9e6537816bfa34`  
		Last Modified: Tue, 30 Mar 2021 21:02:23 GMT  
		Size: 42.1 MB (42065616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26bc0351d047f744512b1f8920863854334f02e11637445a710596e8d9aaa7d`  
		Last Modified: Tue, 30 Mar 2021 21:43:00 GMT  
		Size: 13.3 MB (13265630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cf9228d5dee5e22802266b967dbbb03d58c9f57ab7098649a6337168c4a6fd`  
		Last Modified: Fri, 16 Apr 2021 22:26:43 GMT  
		Size: 186.0 MB (186001704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:17-ea-18-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:89430da7017b85b981ee37f4a547f8f33f120535dcd812d6a9218d0fcb13d5c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.1 MB (238117919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2112e8e2f59e84b3fad9fbf4d2988bb3e20eb710bae394089cf55d0229eb2af0`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 30 Mar 2021 20:50:28 GMT
ADD file:a59a6e0ab925ce07b112d2a2ec9d3f239ea833dc65666a0d1d898d3b048c96ef in / 
# Tue, 30 Mar 2021 20:50:31 GMT
CMD ["/bin/bash"]
# Tue, 30 Mar 2021 21:34:57 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 30 Mar 2021 21:34:58 GMT
ENV JAVA_HOME=/usr/java/openjdk-17
# Tue, 30 Mar 2021 21:34:59 GMT
ENV PATH=/usr/java/openjdk-17/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Mar 2021 21:35:00 GMT
ENV LANG=C.UTF-8
# Fri, 16 Apr 2021 22:40:26 GMT
ENV JAVA_VERSION=17-ea+18
# Fri, 16 Apr 2021 22:41:20 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/18/GPL/openjdk-17-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='272350ce50f4f6f5ff111060a05bafa14f1adfe9ea9f0df06ea1cb242760ed29'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk17/18/GPL/openjdk-17-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='0b65ebc5bcb5e14028c6459bc32158ac530bb41418ca2be95de4da4e64d90df7'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 16 Apr 2021 22:41:21 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7da3223bdf8ee9e05ea4db775be9cb26ab65169aba0ba04ec2c3e0fa7331f0a2`  
		Last Modified: Tue, 30 Mar 2021 20:51:50 GMT  
		Size: 42.0 MB (41995846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e536b6ea357fbefc427ef10b23569012130790959e996d73efed97a345522cf`  
		Last Modified: Tue, 30 Mar 2021 21:41:18 GMT  
		Size: 14.0 MB (14033795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47121d1c52478ab7e2bbddc6e65c19ed7cdc087cbe5c585f49dc922ee2d0edf`  
		Last Modified: Fri, 16 Apr 2021 22:47:11 GMT  
		Size: 182.1 MB (182088278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
