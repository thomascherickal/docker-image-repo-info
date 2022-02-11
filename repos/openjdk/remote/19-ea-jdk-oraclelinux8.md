## `openjdk:19-ea-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:1eab16d020f13682d1a3c88f0ec12d82bf45d9646077156b7f34716cd6f75760
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:206a391a3e1428fdacf84bc62178a032948416cb0d3587642eb305c19aa7f96a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.8 MB (245759177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5114b1af1682a918a2cb188b27313c32d0612ba78543b5661abb13636bb86933`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 11 Feb 2022 18:20:31 GMT
ADD file:636d5d8575ec6ddd380a3bbf41530219d37249378b4abd151d94842377cc55d9 in / 
# Fri, 11 Feb 2022 18:20:32 GMT
CMD ["/bin/bash"]
# Fri, 11 Feb 2022 19:02:04 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Feb 2022 19:02:04 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Fri, 11 Feb 2022 19:02:05 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Feb 2022 19:02:05 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 19:02:05 GMT
ENV JAVA_VERSION=19-ea+8
# Fri, 11 Feb 2022 19:02:16 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/8/GPL/openjdk-19-ea+8_linux-x64_bin.tar.gz'; 			downloadSha256='64f85aad4da5d214002ccbf442b38618b6fae689e66fec2f4a52253d1654683c'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/8/GPL/openjdk-19-ea+8_linux-aarch64_bin.tar.gz'; 			downloadSha256='55bc6f3f3db8a59c77e43ee8ee1ea99d3f121b48d3c7d54cf84f2660a008f047'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 19:02:17 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:010357f4c091049bd23724817a1881f575ff94d35f4c621b4f87b2876049650b`  
		Last Modified: Fri, 11 Feb 2022 18:21:24 GMT  
		Size: 42.1 MB (42105112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1b16b3652a6874ccb11ec011003800c33c1d2f3481ede4da46773eb1415faf`  
		Last Modified: Fri, 11 Feb 2022 19:12:10 GMT  
		Size: 13.5 MB (13514759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8f906ec4868d3d006978653899342fb3dd3e06bffacec3c1deb79962e6e5d4`  
		Last Modified: Fri, 11 Feb 2022 19:12:23 GMT  
		Size: 190.1 MB (190139306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:87ba08557d3068e543d0a2f1e638781ab7543152203b146772e0ad9821300969
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.5 MB (245502247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d1dcd457eedbd01265fa6f9393948a631098a96149c9fa0a4cff5d7eb7a0077`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 11 Feb 2022 18:58:36 GMT
ADD file:8d5a0dcc45ab23c7b507e80b63e5752d94837f490600ce95fb8ba8ed2f7baa2d in / 
# Fri, 11 Feb 2022 18:58:37 GMT
CMD ["/bin/bash"]
# Fri, 11 Feb 2022 19:19:43 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Feb 2022 19:19:43 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Fri, 11 Feb 2022 19:19:44 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Feb 2022 19:19:45 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 19:19:46 GMT
ENV JAVA_VERSION=19-ea+8
# Fri, 11 Feb 2022 19:19:58 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/8/GPL/openjdk-19-ea+8_linux-x64_bin.tar.gz'; 			downloadSha256='64f85aad4da5d214002ccbf442b38618b6fae689e66fec2f4a52253d1654683c'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/8/GPL/openjdk-19-ea+8_linux-aarch64_bin.tar.gz'; 			downloadSha256='55bc6f3f3db8a59c77e43ee8ee1ea99d3f121b48d3c7d54cf84f2660a008f047'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 19:19:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ffdd659a9f05cadeed9c2d5cead839f585163662ca7f847a41fd64bb4e503f0c`  
		Last Modified: Fri, 11 Feb 2022 18:59:38 GMT  
		Size: 42.0 MB (42018804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73433a5e38bf6b279d0c685ed5c2c34fcb8e2d6755228a9c6c3f3a2313bef9b`  
		Last Modified: Fri, 11 Feb 2022 19:35:51 GMT  
		Size: 14.3 MB (14305278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1403c7b5b7c25d968894cbc45a62c641c2d89e8a588229f200c8b9cbc68a2426`  
		Last Modified: Fri, 11 Feb 2022 19:36:06 GMT  
		Size: 189.2 MB (189178165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
