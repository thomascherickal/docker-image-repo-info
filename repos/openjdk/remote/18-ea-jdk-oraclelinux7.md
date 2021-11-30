## `openjdk:18-ea-jdk-oraclelinux7`

```console
$ docker pull openjdk@sha256:45d04b62320be699b50416a2ad3b47a0b624f0df5abed8c9a21a3036f9c7d9e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-ea-jdk-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:591c9be1f470891ab839611777e4721c6c3f895c452eac97fe7cacc64450fa98
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.3 MB (252250932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dd774c09af40ccb64f09951fc7528308fba7d2b6e161a56491e8d0a8ed19fe7`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 24 Nov 2021 22:08:59 GMT
ADD file:8d11c56c80a6b0631722a882ffccf6c4e58297273c4e164138c0f855a670ff79 in / 
# Wed, 24 Nov 2021 22:09:00 GMT
CMD ["/bin/bash"]
# Wed, 24 Nov 2021 22:28:21 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 24 Nov 2021 22:28:21 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 24 Nov 2021 22:28:22 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 22:28:22 GMT
ENV LANG=en_US.UTF-8
# Wed, 24 Nov 2021 22:28:22 GMT
ENV JAVA_VERSION=18-ea+24
# Wed, 24 Nov 2021 22:28:33 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/24/GPL/openjdk-18-ea+24_linux-x64_bin.tar.gz'; 			downloadSha256='be728d2d5f8887ffc348d5a3293938e069c24be47e082a0b61aea61ce328aa03'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/24/GPL/openjdk-18-ea+24_linux-aarch64_bin.tar.gz'; 			downloadSha256='672dcbf3233da1ea245a7991fbeee867817d7024dc5c7e1b533240e642c27626'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 24 Nov 2021 22:28:34 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4ade2748332d656c71c6288f12ab88613792b5c90b329ffdae521095f84faf66`  
		Last Modified: Wed, 24 Nov 2021 22:09:48 GMT  
		Size: 48.3 MB (48331000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6069e51d0239f313c0aee52bbfcdf9d451dba131643e5953161b601efac3d0`  
		Last Modified: Wed, 24 Nov 2021 22:34:59 GMT  
		Size: 15.4 MB (15388482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8995fdb530016a258132f3bb183464aec56296fe46ff60d06a1df1720ece1a`  
		Last Modified: Wed, 24 Nov 2021 22:35:12 GMT  
		Size: 188.5 MB (188531450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-jdk-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:b7bf32aa085096c5c57a18f4fbb1e48deb214b857ae6582b55c50fe477ffcc58
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.9 MB (252868001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6209f8280056eac3097899b56e2f57bde857ff41f0a4640ed406010ab12d258`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 24 Nov 2021 22:01:36 GMT
ADD file:718e42489681d6e9446ec4bb10ba8e24c85d645eb9a303e587f767bedcf668d1 in / 
# Wed, 24 Nov 2021 22:01:37 GMT
CMD ["/bin/bash"]
# Wed, 24 Nov 2021 23:34:39 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 24 Nov 2021 23:34:39 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 24 Nov 2021 23:34:40 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Nov 2021 23:34:41 GMT
ENV LANG=en_US.UTF-8
# Tue, 30 Nov 2021 04:08:05 GMT
ENV JAVA_VERSION=18-ea+25
# Tue, 30 Nov 2021 04:08:22 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/25/GPL/openjdk-18-ea+25_linux-x64_bin.tar.gz'; 			downloadSha256='74a01fc91a33136b6a5d387ecdfc2790ef5e351e3bef869706b288bc9a1df6a2'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/25/GPL/openjdk-18-ea+25_linux-aarch64_bin.tar.gz'; 			downloadSha256='f6f03a12f2c2228a46544ba43b73cd40e4bbb7b5ef857445641d64391d04798c'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Tue, 30 Nov 2021 04:08:23 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:53ff3b63a7657067cd7642c8106127a05a5ea45e3b68cbf830d4120a127e9c82`  
		Last Modified: Wed, 24 Nov 2021 22:02:31 GMT  
		Size: 48.9 MB (48907823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef6b8fb533810fdc95b689d95dd39d5a3f59cb3d3147fddf5bbdf7df183774b`  
		Last Modified: Wed, 24 Nov 2021 23:46:39 GMT  
		Size: 16.5 MB (16464628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3c88ae867632b7ef754897dc08d6b78eacaee4b24059fcc1ac1f4d69d868b4`  
		Last Modified: Tue, 30 Nov 2021 04:20:25 GMT  
		Size: 187.5 MB (187495550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
