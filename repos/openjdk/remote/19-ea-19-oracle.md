## `openjdk:19-ea-19-oracle`

```console
$ docker pull openjdk@sha256:326cc7af8425511726e251958b943590366b6a30404c31e488765d0f154c9aca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-19-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:4cccfd0198d9b5eb99da2362208b0aa3a5bee43d99db6b7f388b2e5f26beb2f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.3 MB (250258435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f580ee0c3f7a3162f8eae424c31350077ce8e340cd16af2b39aa779bd24245e`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 29 Mar 2022 18:35:47 GMT
ADD file:eaa532cad071c531a759e73fd0fd381f440f180ab45b05a74314f10b0374df67 in / 
# Tue, 29 Mar 2022 18:35:47 GMT
CMD ["/bin/bash"]
# Tue, 29 Mar 2022 23:06:25 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Tue, 29 Mar 2022 23:06:25 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Tue, 29 Mar 2022 23:06:26 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 23:06:26 GMT
ENV LANG=C.UTF-8
# Mon, 25 Apr 2022 18:22:13 GMT
ENV JAVA_VERSION=19-ea+19
# Mon, 25 Apr 2022 18:22:42 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/19/GPL/openjdk-19-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='5920845cb577a0883cfbd0bc3a781b5b0a4f71b19a870525c653f9815fa0596b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/19/GPL/openjdk-19-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad9457964256d9d43d6246a0da743a73450231506d0a8a711e28b996b7e6e6e3'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 25 Apr 2022 18:22:44 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e4430e06691f65e516df7d62db0ee5393acea9ade644cc6bc620efef0956dd17`  
		Last Modified: Tue, 29 Mar 2022 18:36:53 GMT  
		Size: 42.1 MB (42113609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ce5342b806de618f4fa582eca53ecee5a73ef976daa060d249227e1927d814`  
		Last Modified: Tue, 29 Mar 2022 23:18:03 GMT  
		Size: 13.5 MB (13524329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c591265d27e4dc92db43ca34ab13f1ce06fa5175d5abd462a05b38b2a52334`  
		Last Modified: Mon, 25 Apr 2022 18:32:54 GMT  
		Size: 194.6 MB (194620497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-19-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:27d66f8e861e0d4f3ecefd859b44c61af17475ceef162225c8638a7247273ce2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.8 MB (249773934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:668e014a0cf07828ed8a1203f5137c2745a767236c4547843f96194305ca3e53`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 29 Mar 2022 18:27:10 GMT
ADD file:08d6d9fea731c201f517e2e96a93c19200773de2ddaa9bed138d10224f7d61e7 in / 
# Tue, 29 Mar 2022 18:27:11 GMT
CMD ["/bin/bash"]
# Wed, 30 Mar 2022 08:57:29 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 30 Mar 2022 08:57:29 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Wed, 30 Mar 2022 08:57:30 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 08:57:31 GMT
ENV LANG=C.UTF-8
# Mon, 25 Apr 2022 18:40:43 GMT
ENV JAVA_VERSION=19-ea+19
# Mon, 25 Apr 2022 18:40:54 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/19/GPL/openjdk-19-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='5920845cb577a0883cfbd0bc3a781b5b0a4f71b19a870525c653f9815fa0596b'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/19/GPL/openjdk-19-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='ad9457964256d9d43d6246a0da743a73450231506d0a8a711e28b996b7e6e6e3'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Mon, 25 Apr 2022 18:40:54 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:293fbd461d2c2a94e5d457aa3c7b18429b8457b06d5c2ad1a57113b1cac6d657`  
		Last Modified: Tue, 29 Mar 2022 18:28:25 GMT  
		Size: 42.0 MB (42019098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d200eb5167ed838a74239544d81e10c3d37a59ea571f23c1d6ed6e0c207cf997`  
		Last Modified: Wed, 30 Mar 2022 09:18:31 GMT  
		Size: 14.3 MB (14293802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c2ae899011005c783985a4898a79a24cce02b0fbabd04f5cd21d227ca15b6e`  
		Last Modified: Mon, 25 Apr 2022 18:57:04 GMT  
		Size: 193.5 MB (193461034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
