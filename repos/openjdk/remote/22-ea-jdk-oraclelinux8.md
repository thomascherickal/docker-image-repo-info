## `openjdk:22-ea-jdk-oraclelinux8`

```console
$ docker pull openjdk@sha256:396794b43ad1f7ae85e03b89802b70328c8d4fbc45065b695bca86f3dfa5e045
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:22-ea-jdk-oraclelinux8` - linux; amd64

```console
$ docker pull openjdk@sha256:f11ec5ff873330eb82124ff70e154117aa0489f9197893181f641159256bb689
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.4 MB (264406039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb9f5d393defd07541c06f1aebc037b08690d33bb21a97a8e7e8d6021f6c064b`
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
# Thu, 12 Oct 2023 22:19:08 GMT
ENV JAVA_VERSION=22-ea+18
# Thu, 12 Oct 2023 22:19:19 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/18/GPL/openjdk-22-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='07830a4cc21745464a68057e8c441e98d4cd673cd02348e9791d9eafe9f3d0df'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/18/GPL/openjdk-22-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='03432a54970a3005c521d34b44a2438ac28f8fe150bf686e28cea6ea9b2a002e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 12 Oct 2023 22:19:20 GMT
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
	-	`sha256:4489c3496ab1b84ba0d0a2b5bce91036812bcfc2b3045b2128ee8c8f4510c729`  
		Last Modified: Thu, 12 Oct 2023 22:20:55 GMT  
		Size: 205.1 MB (205111736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:22-ea-jdk-oraclelinux8` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:ede433604bc64090e096c17bf03fd1e27087a7156912c310d114535443f54df5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262726320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac4034ada3f4a500ecdbf51c95f4b188b9dda354f579e4d5278edbfcd7ff6bfb`
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
# Thu, 12 Oct 2023 15:35:33 GMT
ENV JAVA_VERSION=22-ea+18
# Thu, 12 Oct 2023 15:35:43 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/18/GPL/openjdk-22-ea+18_linux-x64_bin.tar.gz'; 			downloadSha256='07830a4cc21745464a68057e8c441e98d4cd673cd02348e9791d9eafe9f3d0df'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk22/18/GPL/openjdk-22-ea+18_linux-aarch64_bin.tar.gz'; 			downloadSha256='03432a54970a3005c521d34b44a2438ac28f8fe150bf686e28cea6ea9b2a002e'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 12 Oct 2023 15:35:46 GMT
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
	-	`sha256:793599e45b4838306bda56f1a19f73b3e23d86d9ceda357f2902d5cd282beea4`  
		Last Modified: Thu, 12 Oct 2023 15:37:33 GMT  
		Size: 203.4 MB (203396205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
