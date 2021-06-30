## `openjdk:18-ea-jdk-oracle`

```console
$ docker pull openjdk@sha256:043881cdfc7b6cbce9ad0ff9616b75924c74f4ccaa368e79633edfe7f41a696c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-ea-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:ec189832ccaca1d9898902ef40a7b1fceab85a25c4108ecfbfa021a75e86e780
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.6 MB (243577155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b676e01086be1973dcefd2ffd6a1849c795c3897c668db3aeff68958f349e9d3`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 30 Jun 2021 17:23:40 GMT
ADD file:d49890823c4e8287f936eec210400575f79c20f14f048017368faed0584841a6 in / 
# Wed, 30 Jun 2021 17:23:41 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 17:40:57 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 30 Jun 2021 17:40:58 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 30 Jun 2021 17:40:58 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Jun 2021 17:40:58 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 17:40:58 GMT
ENV JAVA_VERSION=18-ea+3
# Wed, 30 Jun 2021 17:42:48 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/3/GPL/openjdk-18-ea+3_linux-x64_bin.tar.gz'; 			downloadSha256='ff917caccd408eacd8758b82a4f9a698d872860d466efb1b23686cfbfb269559'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/3/GPL/openjdk-18-ea+3_linux-aarch64_bin.tar.gz'; 			downloadSha256='db2640da7cfae557c0809f69a643ada97e8048139d2a2e4a4a1f4abe1e762c7b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 30 Jun 2021 17:42:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9660ffb7976c51eb47b4425f6bb95173c170f4fcc442a2bb2b6ba7bf154f6fc8`  
		Last Modified: Wed, 30 Jun 2021 17:25:00 GMT  
		Size: 42.2 MB (42179226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f8b4ca74ea5f238671d4c7981ca7c99e6c70d3fcd8d4d0596ccdf6b8329dbe`  
		Last Modified: Wed, 30 Jun 2021 17:50:04 GMT  
		Size: 13.4 MB (13391447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a80330eeea44214b6272891e82f1cff3f6c6859d3e3fddc893c020e5057899`  
		Last Modified: Wed, 30 Jun 2021 17:50:17 GMT  
		Size: 188.0 MB (188006482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-ea-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:3e1fac20eeab2aed721642bd7ac45c562a034bd9884e1ac40aa1cce35eeafe13
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.0 MB (243040022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3df08c61580d9b8ba19c1c3bd340a717967425a268e3b3031d692110e69a1ea`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 30 Jun 2021 16:40:33 GMT
ADD file:c33580f17660c9afa2637bda7e6cf34d631535b13ffc1535bb21cfb0ab7bdb5c in / 
# Wed, 30 Jun 2021 16:40:33 GMT
CMD ["/bin/bash"]
# Wed, 30 Jun 2021 17:08:45 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 30 Jun 2021 17:08:45 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 30 Jun 2021 17:08:46 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Jun 2021 17:08:46 GMT
ENV LANG=C.UTF-8
# Wed, 30 Jun 2021 17:08:46 GMT
ENV JAVA_VERSION=18-ea+3
# Wed, 30 Jun 2021 17:09:04 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/3/GPL/openjdk-18-ea+3_linux-x64_bin.tar.gz'; 			downloadSha256='ff917caccd408eacd8758b82a4f9a698d872860d466efb1b23686cfbfb269559'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/3/GPL/openjdk-18-ea+3_linux-aarch64_bin.tar.gz'; 			downloadSha256='db2640da7cfae557c0809f69a643ada97e8048139d2a2e4a4a1f4abe1e762c7b'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 30 Jun 2021 17:09:05 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:e02c40d2e97c148eec83200018cd774bcf09562d984b2237577a0bebd5900481`  
		Last Modified: Wed, 30 Jun 2021 16:41:47 GMT  
		Size: 42.0 MB (42045297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c341a81c74999386f57f0e8e08448131a5297ce89816bbfe58e5d804b6e1384`  
		Last Modified: Wed, 30 Jun 2021 17:21:19 GMT  
		Size: 14.2 MB (14179251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8ee57d3358aee1d9bfaee54bc119d64ad2ea5e187d8af39620ab2c915ef60b`  
		Last Modified: Wed, 30 Jun 2021 17:21:34 GMT  
		Size: 186.8 MB (186815474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
