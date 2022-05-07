## `openjdk:19-ea-oraclelinux7`

```console
$ docker pull openjdk@sha256:c2157b18c376abd7ce9057f7a2874cf1398a93a91a3b7fb805c51bbbd4cccbd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:19-ea-oraclelinux7` - linux; amd64

```console
$ docker pull openjdk@sha256:99fceaa5542faaab6b79365f6aed06aa17477263f36a8d26e0fc78e4deb7e39d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.7 MB (257745491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4212334f3fcaee2ac32f4e4d278ced11f8d3d8c7feb2b11059dd4bf4ea84b118`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 29 Mar 2022 18:36:11 GMT
ADD file:b0df42f2bb614be48861be26e670ab6a81c1549d24e64b5e355980adcf0074be in / 
# Tue, 29 Mar 2022 18:36:11 GMT
CMD ["/bin/bash"]
# Tue, 29 Mar 2022 23:06:58 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Tue, 29 Mar 2022 23:06:58 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Tue, 29 Mar 2022 23:06:58 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 23:06:59 GMT
ENV LANG=en_US.UTF-8
# Sat, 07 May 2022 01:20:15 GMT
ENV JAVA_VERSION=19-ea+21
# Sat, 07 May 2022 01:20:24 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='8723353dfc5a3dd34d01b96faddc950c48f450083519a62b287fcb1ef82fc446'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='6e9719e928c6bfa2ed1e3ed7885bc2ff3751e0a8a6c5dde6808dddbd239cba32'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 07 May 2022 01:20:25 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:9347a8f0b30748522f1f50b679f9f2d0c3eea2bb49da98bb4f38a8c8619b7bf8`  
		Last Modified: Tue, 29 Mar 2022 18:37:31 GMT  
		Size: 48.8 MB (48757483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80558a30268385e2f78e93d6dcd977e92f7c76354c6ca130dd3ac4cb4b90f212`  
		Last Modified: Tue, 29 Mar 2022 23:18:51 GMT  
		Size: 14.2 MB (14239096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b90d95a7c484e4396ebff55e887c265d3b137d4155e2284d07351e2344a5415a`  
		Last Modified: Sat, 07 May 2022 01:27:12 GMT  
		Size: 194.7 MB (194748912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:19-ea-oraclelinux7` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:3f1a1d5aa354bf63f8b7f437e69a76372b735ff0cfdc498e911c500acfa30577
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.2 MB (258203960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8a525a30d8c6b916d1e5c92add6dffff820878e204e8d878a5be630c7c1472a`
-	Default Command: `["jshell"]`

```dockerfile
# Tue, 29 Mar 2022 18:27:34 GMT
ADD file:90c167a56275b374fb1719a6f499aea26290701a7baef901065a814af0e9e7c0 in / 
# Tue, 29 Mar 2022 18:27:35 GMT
CMD ["/bin/bash"]
# Wed, 30 Mar 2022 08:58:30 GMT
RUN set -eux; 	yum install -y 		gzip 		tar 				binutils 		freetype fontconfig 	; 	rm -rf /var/cache/yum
# Wed, 30 Mar 2022 08:58:31 GMT
ENV JAVA_HOME=/usr/java/openjdk-19
# Wed, 30 Mar 2022 08:58:32 GMT
ENV PATH=/usr/java/openjdk-19/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 08:58:33 GMT
ENV LANG=en_US.UTF-8
# Sat, 07 May 2022 00:46:55 GMT
ENV JAVA_VERSION=19-ea+21
# Sat, 07 May 2022 00:47:12 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_linux-x64_bin.tar.gz'; 			downloadSha256='8723353dfc5a3dd34d01b96faddc950c48f450083519a62b287fcb1ef82fc446'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk19/21/GPL/openjdk-19-ea+21_linux-aarch64_bin.tar.gz'; 			downloadSha256='6e9719e928c6bfa2ed1e3ed7885bc2ff3751e0a8a6c5dde6808dddbd239cba32'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Sat, 07 May 2022 00:47:13 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:b8909fcd1d3ed60203b3ef173f01925cfd334ae0874f19f3d19876d262428e7e`  
		Last Modified: Tue, 29 Mar 2022 18:29:06 GMT  
		Size: 49.3 MB (49339436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053940d29ef2ce62ec889516ac542e5db9ba471201782b15c2890f3f0be5b92c`  
		Last Modified: Wed, 30 Mar 2022 09:19:27 GMT  
		Size: 15.3 MB (15253020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100c12c7e67439f90cd8576b8db0473a6665f72a0a0ae9bac23412741818505f`  
		Last Modified: Sat, 07 May 2022 00:59:51 GMT  
		Size: 193.6 MB (193611504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
