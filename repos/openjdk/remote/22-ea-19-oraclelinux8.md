## `openjdk:22-ea-19-oraclelinux8`

```console
$ docker pull openjdk@sha256:fdcd8605d1893a8c44ad8058029e3baa8f4d85728b5ab3ca8fb366ebe3afb00c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-ea-19-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:e8ada696009b82ddf72710fe752f58ce2ab1db1697f835a5d06abf595d04e33a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.5 MB (264473687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd203a05159a6dc9ddac66ce02f9ef8ce82d078f654faba404499a0d4c82fa5e`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 12 Oct 2023 21:28:30 GMT
ADD file:3c65f844bba9cf4decac4432464fc55e211e28f5e9753ab337fe057357fee7b5 in / 
# Thu, 12 Oct 2023 21:28:31 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 22:19:07 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 12 Oct 2023 22:19:08 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Thu, 12 Oct 2023 22:19:08 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 22:19:08 GMT
ENV LANG=C.UTF-8
# Fri, 13 Oct 2023 02:02:09 GMT
ENV JAVA_VERSION=22-ea+19
# Fri, 13 Oct 2023 02:02:35 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/19/GPL/openjdk-22-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='70bc0434cc0a8e1fa5351daa062cdd86b29caa784525f22e8a0cc0028e34a157'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/19/GPL/openjdk-22-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='973d8beb242379ed3bec118f7374dc61a99699411c38875ecdf158e506b0a3c0'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 13 Oct 2023 02:02:35 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:210eb976c4c725a4b96ff6ec8a7e848396482dbb1e18d401ee1789c1c6aa6ae0`  
		Last Modified: Thu, 12 Oct 2023 21:30:01 GMT  
		Size: 44.3 MB (44279111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1ad07e4410c408630c3fb5115e2de88151893a626b68399eeac7004b53a1ae`  
		Last Modified: Thu, 12 Oct 2023 22:20:41 GMT  
		Size: 15.0 MB (15015192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abac6306571aa24262275f2fcc7721d5f743ed8ad273b619b590674615f804c1`  
		Last Modified: Fri, 13 Oct 2023 02:06:04 GMT  
		Size: 205.2 MB (205179384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-19-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:05de59ce951329c34a5f4320e6b01d9cb2804953034b130e079a13d6a716bba2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262731978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:059ce233608637d6c6bf5adba9462d70834420f2204b3528d5319b88f701a827`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 12 Oct 2023 11:00:33 GMT
ADD file:b51d9ae1b78eb07ac424bfa71c45180e09ea3a5ed18fbfbcf881fb540bf83e9a in / 
# Thu, 12 Oct 2023 11:00:34 GMT
CMD ["/bin/bash"]
# Thu, 12 Oct 2023 15:35:33 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 12 Oct 2023 15:35:33 GMT
ENV JAVA_HOME=/usr/java/openjdk-22
# Thu, 12 Oct 2023 15:35:33 GMT
ENV PATH=/usr/java/openjdk-22/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 15:35:33 GMT
ENV LANG=C.UTF-8
# Fri, 13 Oct 2023 05:22:05 GMT
ENV JAVA_VERSION=22-ea+19
# Fri, 13 Oct 2023 05:22:50 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/19/GPL/openjdk-22-ea+19_linux-x64_bin.tar.gz'; 			downloadSha256='70bc0434cc0a8e1fa5351daa062cdd86b29caa784525f22e8a0cc0028e34a157'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/19/GPL/openjdk-22-ea+19_linux-aarch64_bin.tar.gz'; 			downloadSha256='973d8beb242379ed3bec118f7374dc61a99699411c38875ecdf158e506b0a3c0'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Fri, 13 Oct 2023 05:22:52 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:89ec84aa94fe6a62fb4e9f51aced09dea3cc4d7979c9f0ebd6b5bd4fd729e04e`  
		Last Modified: Thu, 12 Oct 2023 11:01:48 GMT  
		Size: 43.7 MB (43669807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e397f66df47c7c3f0d7eb2c31f98c331509da0eb0ce59938e0bd38fe4abb900c`  
		Last Modified: Thu, 12 Oct 2023 15:37:20 GMT  
		Size: 15.7 MB (15660308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91797a33eeeb7554f478aecdf362774cf51ecaca09d8c54b28434bc6e6f05b93`  
		Last Modified: Fri, 13 Oct 2023 05:25:23 GMT  
		Size: 203.4 MB (203401863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
