## `openjdk:16-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:cd516c44b5cf5d30f89480e12e2179e01b54f9581a90e1bdd20dcb33ccad90f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:16-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:f1a8b2ed1809803c2850a78139888c103a4e8484aa661eefe41b3508904c4535
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.3 MB (240257663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e4c5a73ccd8681a0fbaf3c8a2e51ba2f41f30f4f3924596b0ff03cfac7e65e`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 13 Oct 2021 18:29:51 GMT
ADD file:3223e5829b65b376c23e1faa6f519d37b0166b38063f91b793a8ed710a39fe33 in / 
# Wed, 13 Oct 2021 18:29:51 GMT
CMD ["/bin/bash"]
# Wed, 13 Oct 2021 18:47:48 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 13 Oct 2021 18:49:48 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Wed, 13 Oct 2021 18:49:48 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 18:49:48 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 18:49:48 GMT
ENV JAVA_VERSION=16.0.2
# Wed, 13 Oct 2021 18:50:00 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 13 Oct 2021 18:50:01 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:58c4eaffce77ac1fb013bf82c91927c631802ad54465ebc9b687b5dc8ee73c02`  
		Last Modified: Wed, 13 Oct 2021 18:31:20 GMT  
		Size: 42.0 MB (41961111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a22c806ee8aa2b360bd5818a4f78bc3da280abb86f3db09805b1daddd78324`  
		Last Modified: Wed, 13 Oct 2021 18:56:49 GMT  
		Size: 13.5 MB (13489427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14afce733284f533ef0231bbf5eac60b0fe3ea5b536fb62f27d5ed8a66cdcbf`  
		Last Modified: Wed, 13 Oct 2021 19:00:05 GMT  
		Size: 184.8 MB (184807125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:16-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:d498187da1cd31c8437127b68fadd6d8099b20a37ccf6315037631da95ffeff4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.3 MB (235342717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f406a2f30aa78e2051959bf597e9c80fde5cc058a9da3001590e64af8b0ee83`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 29 Sep 2021 09:28:21 GMT
ADD file:19a29c4f8accf14e581617044399a0a04fbdf31b2a3dd531b59c72d011deea65 in / 
# Wed, 29 Sep 2021 09:28:21 GMT
CMD ["/bin/bash"]
# Wed, 13 Oct 2021 05:58:48 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 13 Oct 2021 06:04:56 GMT
ENV JAVA_HOME=/usr/java/openjdk-16
# Wed, 13 Oct 2021 06:04:57 GMT
ENV PATH=/usr/java/openjdk-16/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Oct 2021 06:04:58 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 06:04:59 GMT
ENV JAVA_VERSION=16.0.2
# Wed, 13 Oct 2021 06:05:10 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-x64_bin.tar.gz'; 			downloadSha256='6c714ded7d881ca54970ec949e283f43d673a142fda1de79b646ddd619da9c0c'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_linux-aarch64_bin.tar.gz'; 			downloadSha256='1ffb9c7748334945d9056b3324de3f797d906fce4dad86beea955153aa1e28fe'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 13 Oct 2021 06:05:10 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:fbe1b66208e55e97b0e90b882e6fdeed78abb9318897a2d87343840b78e723ef`  
		Last Modified: Wed, 29 Sep 2021 09:29:46 GMT  
		Size: 41.9 MB (41883345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076e889c44db9131098a7368fb924c97ba81cb10aee46f9c273b2076baab08f5`  
		Last Modified: Wed, 13 Oct 2021 06:23:16 GMT  
		Size: 14.3 MB (14270423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49d132e602acc15ad57247a05d1a4174849f92e8835af3ac415828b8a789de3`  
		Last Modified: Wed, 13 Oct 2021 06:31:56 GMT  
		Size: 179.2 MB (179188949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
