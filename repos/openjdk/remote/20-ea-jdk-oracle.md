## `openjdk:20-ea-jdk-oracle`

```console
$ docker pull openjdk@sha256:7df4325f1ff582a057244a45853eaa791d2976e5b01b11f6e6dc1792ae284860
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `openjdk:20-ea-jdk-oracle` - linux; amd64

```console
$ docker pull openjdk@sha256:a145b5191c96b982398ded1d0fdc27a0d6031792572b8f5e5ab89f90ce5ddd0c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.9 MB (249879997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49cafc33e9fad9b5dd876263b5390233b999d0a52c008f8217d8d6979827e8fe`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Jun 2022 17:20:45 GMT
ADD file:03d0377f5864198b250372de990ebf0ef7597cfdcc2e18421e8e0025394a7572 in / 
# Thu, 30 Jun 2022 17:20:46 GMT
CMD ["/bin/bash"]
# Thu, 30 Jun 2022 17:37:33 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 30 Jun 2022 17:37:33 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Thu, 30 Jun 2022 17:37:33 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jun 2022 17:37:34 GMT
ENV LANG=C.UTF-8
# Thu, 30 Jun 2022 17:37:34 GMT
ENV JAVA_VERSION=20-ea+3
# Thu, 30 Jun 2022 17:37:43 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/3/GPL/openjdk-20-ea+3_linux-x64_bin.tar.gz'; 			downloadSha256='8f930cbbf2c85c0cfe87eef8646d1e038fe51d19132613e868e96118b1e0f8d0'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/3/GPL/openjdk-20-ea+3_linux-aarch64_bin.tar.gz'; 			downloadSha256='d7b270b059fe08487492d38760e0e821b3a7be20864205d7ab0b5e5206109bda'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 30 Jun 2022 17:37:44 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:337897a5aaf7b54e691e2ed305fbf00e0e8933d5a8a3c07d6fbb95f10b15c644`  
		Last Modified: Thu, 30 Jun 2022 17:21:37 GMT  
		Size: 39.2 MB (39221672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1e7c755c4cccc19ca62372088ce86de7711ff0e0e2e7e18f65711eb2299602`  
		Last Modified: Thu, 30 Jun 2022 17:45:09 GMT  
		Size: 13.5 MB (13509384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63012b5e715f55e4ffdc7118eab9c8304685e8554f82b7e884b9afc9f7bd4ced`  
		Last Modified: Thu, 30 Jun 2022 17:45:22 GMT  
		Size: 197.1 MB (197148941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `openjdk:20-ea-jdk-oracle` - linux; arm64 variant v8

```console
$ docker pull openjdk@sha256:1acf50078f758ec39001e19292d8ca88743539db9bc361251f2139b983f899e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.3 MB (248319901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cad3a37cf3c5df11dc99487dfb30bf0111e13276d800b4ee9d30ef9e35db057`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 30 Jun 2022 17:40:34 GMT
ADD file:deb746f3cc547a36a34f3bfe68510bbd6f8a3b2da72bcca3cce36dfe0e519e77 in / 
# Thu, 30 Jun 2022 17:40:35 GMT
CMD ["/bin/bash"]
# Thu, 30 Jun 2022 18:00:54 GMT
RUN set -eux; 	microdnf install 		gzip 		tar 				binutils 		freetype fontconfig 	; 	microdnf clean all
# Thu, 30 Jun 2022 18:00:54 GMT
ENV JAVA_HOME=/usr/java/openjdk-20
# Thu, 30 Jun 2022 18:00:55 GMT
ENV PATH=/usr/java/openjdk-20/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Jun 2022 18:00:56 GMT
ENV LANG=C.UTF-8
# Thu, 30 Jun 2022 18:00:57 GMT
ENV JAVA_VERSION=20-ea+3
# Thu, 30 Jun 2022 18:01:18 GMT
RUN set -eux; 		arch="$(objdump="$(command -v objdump)" && objdump --file-headers "$objdump" | awk -F '[:,]+[[:space:]]+' '$1 == "architecture" { print $2 }')"; 	case "$arch" in 		'i386:x86-64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/3/GPL/openjdk-20-ea+3_linux-x64_bin.tar.gz'; 			downloadSha256='8f930cbbf2c85c0cfe87eef8646d1e038fe51d19132613e868e96118b1e0f8d0'; 			;; 		'aarch64') 			downloadUrl='https://download.java.net/java/early_access/jdk20/3/GPL/openjdk-20-ea+3_linux-aarch64_bin.tar.gz'; 			downloadSha256='d7b270b059fe08487492d38760e0e821b3a7be20864205d7ab0b5e5206109bda'; 			;; 		*) echo >&2 "error: unsupported architecture: '$arch'"; exit 1 ;; 	esac; 		curl -fL -o openjdk.tgz "$downloadUrl"; 	echo "$downloadSha256 *openjdk.tgz" | sha256sum --strict --check -; 		mkdir -p "$JAVA_HOME"; 	tar --extract 		--file openjdk.tgz 		--directory "$JAVA_HOME" 		--strip-components 1 		--no-same-owner 	; 	rm openjdk.tgz*; 		rm -rf "$JAVA_HOME/lib/security/cacerts"; 	ln -sT /etc/pki/ca-trust/extracted/java/cacerts "$JAVA_HOME/lib/security/cacerts"; 		ln -sfT "$JAVA_HOME" /usr/java/default; 	ln -sfT "$JAVA_HOME" /usr/java/latest; 	for bin in "$JAVA_HOME/bin/"*; do 		base="$(basename "$bin")"; 		[ ! -e "/usr/bin/$base" ]; 		alternatives --install "/usr/bin/$base" "$base" "$bin" 20000; 	done; 		java -Xshare:dump; 		fileEncoding="$(echo 'System.out.println(System.getProperty("file.encoding"))' | jshell -s -)"; [ "$fileEncoding" = 'UTF-8' ]; rm -rf ~/.java; 	javac --version; 	java --version
# Thu, 30 Jun 2022 18:01:19 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c7107c973a1b04b1f048e43f460fd4f030df5f2e53fce3dfb8a13dc7fefdb4b0`  
		Last Modified: Thu, 30 Jun 2022 17:41:32 GMT  
		Size: 38.0 MB (38023864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a33b6e144a0eee25610c802e234489b8afda2108ce38e5f76ee4d79e5e45ff`  
		Last Modified: Thu, 30 Jun 2022 18:15:30 GMT  
		Size: 14.3 MB (14303308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a15aa1dc5096392961caa44354931a26b8fd9919dab56c9f6846f06efeb9403`  
		Last Modified: Thu, 30 Jun 2022 18:15:47 GMT  
		Size: 196.0 MB (195992729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
