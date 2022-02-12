## `openjdk:18-oraclelinux8`

```console
$ docker pull openjdk@sha256:9d3bb05e4b4cb976933f11e79819decabfd37d85651f5fce4a107f6b17e052a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:d15718c1f14e027dc4cd6e3ee8662fbfcbb7e9c5ae047bfbce8847b3baaa9e9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244288666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aecf72a3a839d0103789ac1e29c571ca33c4789d759c4ec393819da1732c0f70`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 11 Feb 2022 18:20:31 GMT
ADD file:636d5d8575ec6ddd380a3bbf41530219d37249378b4abd151d94842377cc55d9 in / 
# Fri, 11 Feb 2022 18:20:32 GMT
CMD ["/bin/bash"]
# Fri, 11 Feb 2022 19:02:04 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Feb 2022 19:02:43 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Fri, 11 Feb 2022 19:02:43 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Feb 2022 19:02:44 GMT
ENV LANG=C.UTF-8
# Fri, 11 Feb 2022 23:51:26 GMT
ENV JAVA_VERSION=18-ea+35
# Fri, 11 Feb 2022 23:51:45 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/35/GPL/openjdk-18-ea+35_linux-x64_bin.tar.gz'; 			downloadSha256='62a711fdc1a8f7051551113d62f8cc7e3be42e57335d11d605dab060f29a12e2'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/35/GPL/openjdk-18-ea+35_linux-aarch64_bin.tar.gz'; 			downloadSha256='cf0298eeac8e0d1d93fb1615916e08c12cd1a0e372a132cec2e66b2a30de6815'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 11 Feb 2022 23:51:46 GMT
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
	-	`sha256:f86b23c3b56d41d702c95b08ce3bee75de206be11df04b8bb18cf40568fa0502`  
		Last Modified: Sat, 12 Feb 2022 00:14:57 GMT  
		Size: 188.7 MB (188668795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:48b1bfdc146145a1de65cf34338b5d99e2a09c2b06d933f9875e2504b26c6ec8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.9 MB (243929601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9892b28543aa139ab9ff9fb1390e97d0689061427ed910a238f10f8435f6711c`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 11 Feb 2022 18:58:36 GMT
ADD file:8d5a0dcc45ab23c7b507e80b63e5752d94837f490600ce95fb8ba8ed2f7baa2d in / 
# Fri, 11 Feb 2022 18:58:37 GMT
CMD ["/bin/bash"]
# Fri, 11 Feb 2022 19:19:43 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 11 Feb 2022 19:20:44 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Fri, 11 Feb 2022 19:20:44 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Feb 2022 19:20:45 GMT
ENV LANG=C.UTF-8
# Sat, 12 Feb 2022 00:08:53 GMT
ENV JAVA_VERSION=18-ea+35
# Sat, 12 Feb 2022 00:09:07 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/35/GPL/openjdk-18-ea+35_linux-x64_bin.tar.gz'; 			downloadSha256='62a711fdc1a8f7051551113d62f8cc7e3be42e57335d11d605dab060f29a12e2'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/35/GPL/openjdk-18-ea+35_linux-aarch64_bin.tar.gz'; 			downloadSha256='cf0298eeac8e0d1d93fb1615916e08c12cd1a0e372a132cec2e66b2a30de6815'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 12 Feb 2022 00:09:08 GMT
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
	-	`sha256:0fbd47b9449a6269d5cc52132b96fa8b070bb9faa6d6cdf0a04faf2e23948837`  
		Last Modified: Sat, 12 Feb 2022 00:33:11 GMT  
		Size: 187.6 MB (187605519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
