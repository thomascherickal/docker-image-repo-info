## `openjdk:19-oracle`

```console
$ docker pull openjdk@sha256:bf4582264c97c50a41ad8215d7399d3e4ba722ba59c0855848f4c202489ee5c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:289bcaff8a4e9dc2cd52200b926203583e6fda087efe820819ffaae41b81ccc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.7 MB (248727757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bd51d5a8051e42cded75e5439143193bc7ac7013c8e6d863387bc494bfeaed6`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 24 Mar 2022 22:26:17 GMT
ADD file:ebb4986af4fcca0d00738e77d2c814e70536c01a0e02eef98c71e9e3a56c0abd in / 
# Thu, 24 Mar 2022 22:26:18 GMT
CMD ["/bin/bash"]
# Fri, 25 Mar 2022 01:16:47 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Fri, 25 Mar 2022 01:16:47 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Fri, 25 Mar 2022 01:16:47 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 25 Mar 2022 01:16:47 GMT
ENV LANG=C.UTF-8
# Fri, 25 Mar 2022 01:16:47 GMT
ENV JAVA_VERSION=19-ea+14
# Fri, 25 Mar 2022 01:16:57 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/14/GPL/openjdk-19-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='7c64317f728ce251b1fa6fcc612bbc5e4fac4d2862cf0f9b9edd98800072b6bc'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/14/GPL/openjdk-19-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='166aaa023baf2fff6484465efd16040557b4bbd57362409d730acec5d01fe749'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 25 Mar 2022 01:16:58 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:1de6f411eccf5041d90362d2d035abf0e59cf91dce4eacbc37ef0aa52f5b5920`  
		Last Modified: Thu, 24 Mar 2022 22:27:23 GMT  
		Size: 42.1 MB (42111629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbc239737191ccc9950c0b7c7a0aa6dac0a92906c45c8c72d511820cf4cd3b6`  
		Last Modified: Fri, 25 Mar 2022 01:24:51 GMT  
		Size: 13.5 MB (13530268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64eccc23cb93603515853d28fe7365150ee2437fddfcbe5a5e41019eefd959f1`  
		Last Modified: Fri, 25 Mar 2022 01:25:03 GMT  
		Size: 193.1 MB (193085860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:dd60ed8fd43d4ec6b51145a99047294cc469d54011f79166dc3be3fbb0277192
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.4 MB (248432264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34bdaeacd62a10c28737c3f8a72c154f1f70bf22df8d8d801e28dc8b21353f45`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 24 Mar 2022 22:21:09 GMT
ADD file:1eaca9dccdbe88c4fac0b484a625100443af30879cf6cba7b5615db77745b0c7 in / 
# Thu, 24 Mar 2022 22:21:10 GMT
CMD ["/bin/bash"]
# Thu, 24 Mar 2022 22:45:15 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 24 Mar 2022 22:45:16 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Thu, 24 Mar 2022 22:45:17 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 22:45:18 GMT
ENV LANG=C.UTF-8
# Thu, 24 Mar 2022 22:45:19 GMT
ENV JAVA_VERSION=19-ea+14
# Thu, 24 Mar 2022 22:45:30 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/14/GPL/openjdk-19-ea+14_linux-x64_bin.tar.gz'; 			downloadSha256='7c64317f728ce251b1fa6fcc612bbc5e4fac4d2862cf0f9b9edd98800072b6bc'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/14/GPL/openjdk-19-ea+14_linux-aarch64_bin.tar.gz'; 			downloadSha256='166aaa023baf2fff6484465efd16040557b4bbd57362409d730acec5d01fe749'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 24 Mar 2022 22:45:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c11319b13f376dfb3fa1ee22d0047cfb7157eba4ba2786653cb29ac6defcb93c`  
		Last Modified: Thu, 24 Mar 2022 22:22:26 GMT  
		Size: 42.0 MB (42018948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d7710250d8de942c9ab085f8642e5e854d0b85b2578079aa2a8f4aaac0bf73`  
		Last Modified: Thu, 24 Mar 2022 23:01:12 GMT  
		Size: 14.3 MB (14293656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abace735fa41f5dd83fa3348a2038605a3ba8cd5d92b935b9494d1ece1b1910`  
		Last Modified: Thu, 24 Mar 2022 23:01:29 GMT  
		Size: 192.1 MB (192119660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
