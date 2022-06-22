## `openjdk:19-ea-27-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:360449b3f7d30faa728503efd4b9672e65b4911bd0527bc0cefef0bffb960828
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-27-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:093fb206087db64e973ba5e58d662e118a5cc62f802afbd48ab5506182c81b90
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.1 MB (259126795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d82c872f71ea0bef0fd1d77bdc61e4e6e5074a22b556352ded538a3e3800ea9e`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 16 Jun 2022 01:20:22 GMT
ADD file:5e615d6d49ec50cba937fa86f5fb7d6a4a7e680b2b4f5b659e879b95304c0417 in / 
# Thu, 16 Jun 2022 01:20:22 GMT
CMD ["/bin/bash"]
# Thu, 16 Jun 2022 01:22:07 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 16 Jun 2022 01:23:30 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 16 Jun 2022 01:23:30 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Jun 2022 01:23:30 GMT
ENV LANG=en_US.UTF-8
# Wed, 22 Jun 2022 01:22:05 GMT
ENV JAVA_VERSION=19-ea+27
# Wed, 22 Jun 2022 01:22:15 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/27/GPL/openjdk-19-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='d88a9e824ce2c65fd634463856a6af2e8aad09a3b005a6ae9f3529b972d184c4'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/27/GPL/openjdk-19-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='7e93f0cde43b50161e5817e8a12907f5a2e74dbd63a4fa99d059ba4afdab02ae'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 22 Jun 2022 01:22:16 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:63183c9b4598e16c4cef95f706d50ff6c928de41f391cd513495b27eaa27bf89`  
		Last Modified: Thu, 16 Jun 2022 01:21:08 GMT  
		Size: 48.8 MB (48757931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb5aec2fa88dbfc29b4af04e13302acbb1298cf96be28433c81b5293be618be`  
		Last Modified: Thu, 16 Jun 2022 01:31:20 GMT  
		Size: 14.2 MB (14236378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3f96b050e5cfcb180869e1838d43c90f6f7303c31bf630b801d5553b73d3e4`  
		Last Modified: Wed, 22 Jun 2022 01:34:20 GMT  
		Size: 196.1 MB (196132486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-27-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:517150c7e674b67ce3ffc70ad85e64e926f8fbcfe64bdd6c3d4861aa69c67770
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259590668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a70bf546f4b84a731f6edb691dee80aa8a00c9e296f9cf5f6ec13a9114d7c43d`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 16 Jun 2022 01:12:02 GMT
ADD file:3c802f9fbd1a9a4878df064e2b268b017930633407658a3f9d29e53eb74552fa in / 
# Thu, 16 Jun 2022 01:12:03 GMT
CMD ["/bin/bash"]
# Thu, 16 Jun 2022 02:52:59 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Thu, 16 Jun 2022 02:54:08 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 16 Jun 2022 02:54:08 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Jun 2022 02:54:09 GMT
ENV LANG=en_US.UTF-8
# Wed, 22 Jun 2022 02:15:45 GMT
ENV JAVA_VERSION=19-ea+27
# Wed, 22 Jun 2022 02:16:02 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/27/GPL/openjdk-19-ea+27_linux-x64_bin.tar.gz'; 			downloadSha256='d88a9e824ce2c65fd634463856a6af2e8aad09a3b005a6ae9f3529b972d184c4'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/27/GPL/openjdk-19-ea+27_linux-aarch64_bin.tar.gz'; 			downloadSha256='7e93f0cde43b50161e5817e8a12907f5a2e74dbd63a4fa99d059ba4afdab02ae'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 22 Jun 2022 02:16:03 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9071f63390163e069a5245aea05c5a92f0dd4a4a48483db57c4c3c0d557be5e7`  
		Last Modified: Thu, 16 Jun 2022 01:12:57 GMT  
		Size: 49.3 MB (49343296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e709d91969def8bffeaecd5e24c79283c0850fbc3e9924fe9ae16ad997e75ac`  
		Last Modified: Thu, 16 Jun 2022 03:07:48 GMT  
		Size: 15.3 MB (15264634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0864c17d37c66daab1078994a4e5527c820e9fcca545958327e0a241203f4ec1`  
		Last Modified: Wed, 22 Jun 2022 02:35:17 GMT  
		Size: 195.0 MB (194982738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
