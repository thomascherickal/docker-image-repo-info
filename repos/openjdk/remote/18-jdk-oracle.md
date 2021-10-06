## `openjdk:18-jdk-oracle`

```console
$ docker pull openjdk@sha256:2fe672edaa8cbf588cddbee9fe28cba73da9f4ffa0f7003050c8e51a4cc115e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:18-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:b1b1385e71f56522d1ec8b8ca81a1df0f7747cccf4c50f90d86003b89517f036
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.3 MB (243348458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:612fa4e2c4c598cb556bf46819fd5487a1bb0089304dd9ac74f49013d05dc7c0`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 29 Sep 2021 16:28:05 GMT
ADD file:99c665dc5bddb30b592aa86f66d1256f41b468201a93afe0c6164edb42c388c4 in / 
# Wed, 29 Sep 2021 16:28:06 GMT
CMD ["/bin/bash"]
# Wed, 29 Sep 2021 16:53:34 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 29 Sep 2021 16:53:34 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 29 Sep 2021 16:53:34 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 16:53:34 GMT
ENV LANG=C.UTF-8
# Wed, 06 Oct 2021 18:28:37 GMT
ENV JAVA_VERSION=18-ea+17
# Wed, 06 Oct 2021 18:28:48 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/17/GPL/openjdk-18-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='3a79fd0700f8e27538bb6cdbef4f630be0efc78686b6f4c3003dcea1177a237a'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/17/GPL/openjdk-18-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='9ff48be04860c0632addb495dcba1d4fe519d306edd4165b17848a8d340d0340'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 06 Oct 2021 18:28:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:6540cb32758bf3f150d56508f216b26487b14ac6fd20b1c92f1e1c8357730ea9`  
		Last Modified: Wed, 29 Sep 2021 16:29:48 GMT  
		Size: 42.0 MB (41963002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3acb1bb05d773c14486a356ac78716bf3e9e5b34aefb39b421cc776aea66e606`  
		Last Modified: Wed, 29 Sep 2021 17:02:29 GMT  
		Size: 13.5 MB (13490694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceafc2a37e5adbfac09e26c7ef86d1dcd6d3f7f911c89bda86845e3ad64b4550`  
		Last Modified: Wed, 06 Oct 2021 18:36:16 GMT  
		Size: 187.9 MB (187894762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:18-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:c555126bab4d6d0feda1ed47e3790bed53a7ffb8d17f7415c90b5a8f0d5e0fcf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.9 MB (242947719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d949a61579a7de7f035f0afe8a9b333b3cf0a1733953f9938a963bb41c0d58a`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 29 Sep 2021 09:28:21 GMT
ADD file:19a29c4f8accf14e581617044399a0a04fbdf31b2a3dd531b59c72d011deea65 in / 
# Wed, 29 Sep 2021 09:28:21 GMT
CMD ["/bin/bash"]
# Wed, 29 Sep 2021 10:13:29 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Wed, 29 Sep 2021 10:13:30 GMT
ENV JAVA_HOME=/usr/java/openjdk-18
# Wed, 29 Sep 2021 10:13:30 GMT
ENV PATH=/usr/java/openjdk-18/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 10:13:30 GMT
ENV LANG=C.UTF-8
# Wed, 06 Oct 2021 18:06:57 GMT
ENV JAVA_VERSION=18-ea+17
# Wed, 06 Oct 2021 18:07:06 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/17/GPL/openjdk-18-ea+17_linux-x64_bin.tar.gz'; 			downloadSha256='3a79fd0700f8e27538bb6cdbef4f630be0efc78686b6f4c3003dcea1177a237a'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk18/17/GPL/openjdk-18-ea+17_linux-aarch64_bin.tar.gz'; 			downloadSha256='9ff48be04860c0632addb495dcba1d4fe519d306edd4165b17848a8d340d0340'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Wed, 06 Oct 2021 18:07:06 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:fbe1b66208e55e97b0e90b882e6fdeed78abb9318897a2d87343840b78e723ef`  
		Last Modified: Wed, 29 Sep 2021 09:29:46 GMT  
		Size: 41.9 MB (41883345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fe2b96b9211b7b369c53846fe42fa00426fa23a6d736fb50873c69ffc8b3c9`  
		Last Modified: Wed, 29 Sep 2021 10:29:47 GMT  
		Size: 14.3 MB (14275215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2147582da5dc82547ccced334e8b8fa6a833b7277f381fa1b8f547d59ef509c9`  
		Last Modified: Wed, 06 Oct 2021 18:21:02 GMT  
		Size: 186.8 MB (186789159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
